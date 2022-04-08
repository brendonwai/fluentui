## API Report File for "@fluentui/react-focus"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import type { IRefObject } from '@fluentui/utilities';
import type { Point } from '@fluentui/utilities';
import * as React_2 from 'react';

// @public (undocumented)
export class FocusZone extends React_2.Component<IFocusZoneProps> implements IFocusZone {
    constructor(props: IFocusZoneProps);
    // (undocumented)
    componentDidMount(): void;
    // (undocumented)
    componentDidUpdate(): void;
    // (undocumented)
    componentWillUnmount(): void;
    // (undocumented)
    static defaultProps: IFocusZoneProps;
    focus(forceIntoFirstElement?: boolean): boolean;
    focusElement(element: HTMLElement, forceAlignment?: boolean): boolean;
    focusLast(): boolean;
    static getOuterZones(): number;
    // (undocumented)
    render(): React_2.ReactNode;
    setFocusAlignment(point: Point): void;
}

// @public (undocumented)
export enum FocusZoneDirection {
    bidirectional = 2,
    domOrder = 3,
    horizontal = 1,
    vertical = 0
}

// @public (undocumented)
export const FocusZoneTabbableElements: {
    none: 0;
    all: 1;
    inputOnly: 2;
};

// @public (undocumented)
export type FocusZoneTabbableElements = typeof FocusZoneTabbableElements[keyof typeof FocusZoneTabbableElements];

// @public
export interface IFocusZone {
    focus(forceIntoFirstElement?: boolean): boolean;
    focusElement(childElement?: HTMLElement, forceAlignment?: boolean): boolean;
    focusLast(): boolean;
    setFocusAlignment(point: Point): void;
}

// @public
export interface IFocusZoneProps extends React_2.HTMLAttributes<HTMLElement> {
    allowFocusRoot?: boolean;
    // @deprecated
    allowTabKey?: boolean;
    // @deprecated
    ariaDescribedBy?: string;
    // @deprecated
    ariaLabelledBy?: string;
    as?: React_2.ElementType;
    checkForNoWrap?: boolean;
    className?: string;
    componentRef?: IRefObject<IFocusZone>;
    // @deprecated
    defaultActiveElement?: string;
    defaultTabbableElement?: string | ((root: HTMLElement) => HTMLElement);
    direction?: FocusZoneDirection;
    disabled?: boolean;
    // @deprecated
    doNotAllowFocusEventToPropagate?: boolean;
    // @deprecated
    elementRef?: React_2.Ref<HTMLElement>;
    // @deprecated
    elementType?: any;
    handleTabKey?: FocusZoneTabbableElements;
    isCircularNavigation?: boolean;
    // @deprecated
    isInnerZoneKeystroke?: (ev: React_2.KeyboardEvent<HTMLElement>) => boolean;
    onActiveElementChanged?: (element?: HTMLElement, ev?: React_2.FocusEvent<HTMLElement>) => void;
    // @deprecated
    onBeforeFocus?: (childElement?: HTMLElement) => boolean;
    onFocus?: (event: React_2.FocusEvent<HTMLElement>) => void;
    // @deprecated
    onFocusNotification?: () => void;
    pagingSupportDisabled?: boolean;
    preventDefaultWhenHandled?: boolean;
    preventFocusRestoration?: boolean;
    // @deprecated (undocumented)
    rootProps?: React_2.HTMLAttributes<HTMLDivElement>;
    shouldEnterInnerZone?: (ev: React_2.KeyboardEvent<HTMLElement>) => boolean;
    shouldFocusInnerElementWhenReceivedFocus?: boolean;
    shouldFocusOnMount?: boolean;
    shouldInputLoseFocusOnArrowKey?: (inputElement: HTMLInputElement) => boolean;
    shouldRaiseClicks?: boolean;
    shouldRaiseClicksOnEnter?: boolean;
    shouldRaiseClicksOnSpace?: boolean;
    shouldReceiveFocus?: (childElement?: HTMLElement) => boolean;
    shouldResetActiveElementWhenTabFromZone?: boolean;
    stopFocusPropagation?: boolean;
}

// (No @packageDocumentation comment for this package)

```